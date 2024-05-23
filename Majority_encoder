// Majority Encoder 
library IEEE;
use IEEE.std_logic_1164.all;

entity majority is
  port(
    votes : in std_logic_vector(2 downto 0);
    y : out std_logic
  );
end majority;

architecture synth of majority is
begin
  process(votes)
  begin
    if ( (votes(0) = '1' and votes(1) = '1') or
         (votes(0) = '1' and votes(2) = '1') or
         (votes(1) = '1' and votes(2) = '1') ) then
      y <= '1';
    else
      y <= '0';
    end if;
  end process;
end synth;
